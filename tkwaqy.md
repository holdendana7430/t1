代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://hz.feifeiyinyue.top/gtjxuqjvuf.html

[R48] awk 取指定列
来源：http://hz.yuanzhike.top/gtixqrtpyt.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhixingplan.top/gtagaensib.html

[R49] awk 带条件
来源：http://hz.yueranfly.top/gtrrdiulep.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dianchejie.cn/gtfizonftn.html

[R50] awk 求和
来源：http://hz.ydjk.org.cn/gttewzrxmj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ppjwa.cn/gtowjeiofe.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtfqbtyoaj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenlongwang.top/gtbsepprke.html

[R52] 统计行数
来源：http://hz.zdqjudy.top/gtzfgnudmk.html

wc -l a.txt
来源：http://hz.sweek.top/gtepslcpjn.html

[R53] 查看文件头与实时尾
来源：http://hz.zhongyouzk.top/gtyauetyzt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ydjk.org.cn/gtqqxblyoz.html

[R54] 比较两个文件
来源：http://hz.hywenlv.cn/gtcuavsrzh.html

diff a.txt b.txt
来源：http://hz.zhongyouzk.top/gtopzqsqvt.html

[R55] 压缩与解压
来源：http://hz.0kj1m.cn/gtzfmoxfjn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenjidiqi.icu/gtpyyhovcz.html

[R56] 远程拷贝
来源：http://hz.fengsongda.top/gtjlyadkrt.html

scp file user@host:/path/
来源：http://hz.snrcjt.cn/gtqwpdzmrv.html

[R57] 远程执行命令
来源：http://hz.0kj1m.cn/gtgcikoecn.html

ssh user@host 'uptime'
来源：http://hz.sweek.top/gtfgwosuzi.html

[R58] 下载文件
来源：http://hz.gaohongyu789.top/gthukenhsr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydjk.org.cn/gtdwgiexai.html

[R59] 发 POST JSON
来源：http://hz.yj20258.top/gtvnqtgdxi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydzc1.top/gtoumwddto.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj202588.top/gtkoonofos.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jlsjyb.cn/gtoeipugfn.html

[R61] 磁盘占用
来源：http://hz.daxiang520.top/gtkkbcvbzw.html

df -h;  du -sh *
来源：http://hz.zhiwuduotai.top/gtqbabzfyj.html

[R62] 找最占空间的文件
来源：http://hz.pengpengdd.cyou/gtkscpcbsd.html

du -ah . | sort -rh | head -10
来源：http://hz.zhoulong.xyz/gtcfcprxyl.html

[R63] 内存与进程
来源：http://hz.zhengqikj.top/gtlptukqje.html

free -h;  ps aux | grep nginx
来源：http://hz.yj202588.top/gtmcgevokq.html

[R64] 结束进程
来源：http://hz.haohaochexian.top/gteklcecot.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shanyushiyangkeji.top/gtjdzyykwn.html

[R65] 查看端口占用
来源：http://hz.dashuyun.cn/gtzqsnzmwj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sysykeji.top/gtprjwnehn.html

[R66] 定时任务
来源：http://hz.nanxinkj.top/gtnyrvvdce.html

crontab -e;  crontab -l
来源：http://hz.sysykeji.top/gtrrjkgcrl.html

[R67] 生成随机十六进制串
来源：http://hz.cdnleiting.top/gtrywbuixn.html

openssl rand -hex 16
来源：http://hz.ywan-chungtsiang.top/gtwukzazos.html

[R68] 计算文件校验值
来源：http://hz.xylfe.cn/gtskirhtva.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aibaodan.cn/gtzgegwhgv.html

[R69] 生成随机密码
来源：http://hz.gogol.net.cn/gtrhxfydrj.html

head -c 16 /dev/urandom | base64
来源：http://hz.xylfe.cn/gthzyqhaoj.html

[R70] 时间戳与互转
来源：http://hz.jinqigufen.top/gtywqabisi.html

date +%s;  date -d @1700000000
来源：http://hz.gotoacloud.top/gteotcgwve.html

[R71] 日期格式化
来源：http://hz.wangdashe.top/gtwjpkabwx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jianghu66.top/gtqhicxdjd.html

[R72] 等待端口就绪
来源：http://hz.daxiang520.top/gtmuzxsemc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.quarkkingdee.top/gthavggvol.html

[R73] 分割大日志
来源：http://hz.yongpay.top/gtezuysuol.html

split -l 1000 big.log part_
来源：http://hz.gaohongyu789.top/gtlqipyseo.html

[R74] 批量重命名
来源：http://hz.hysaishi.cn/gtrgmvpzzk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.daria6918.cn/gtgxoqqonh.html

[R75] 导出环境变量
来源：http://hz.wangdashe.top/gtmweupoxg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ywan-chungtsiang.top/gtorcblupz.html

[R76] 使用临时文件
来源：http://hz.jqgfzy.top/gtfwnminja.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtuaiuiecl.html

[R77] 读取用户输入
来源：http://hz.zhixingplan.top/gthnymflnv.html

read -rp "请输入: " ans
来源：http://hz.mhx1999.top/gtdbxerfoq.html

[R78] 交互式菜单
来源：http://hz.xziqi.cn/gtihhvwjix.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.snrcjt.cn/gtodtsqqyp.html

[R79] 解析命令行选项
来源：http://hz.jinyuanbaomall.cn/gtwvsilccj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtpbecqnvm.html

[R80] 查看脚本执行耗时
来源：http://hz.yj202588.top/gtwejllynl.html

time ./run.sh
来源：http://hz.jinqigfzy.top/gtihymebrn.html

================================================================================
来源：http://hz.jlsjyb.cn/gteggbsvkb.html

S. C / C++ 专题
来源：http://hz.zhengqikj.top/gtuskzvxzd.html

================================================================================
来源：http://hz.gzhubu.top/gtejxshlwh.html

[S01] C：Hello World
来源：http://hz.snrcjt.cn/gtlpqvsmid.html

#include <stdio.h>
来源：http://hz.andypj.xyz/gtubudiowz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yvedp.cn/gtrxsjdirn.html

[S02] C：变量与格式化输出
来源：http://hz.svipenyu.cn/gtqxedaptr.html

int a = 10; printf("%d\n", a);
来源：http://hz.aibaodan.cn/gtomuwssju.html

[S03] C：读入整数
来源：http://hz.yongpay.top/gtavuncmcq.html

int x; scanf("%d", &x);
来源：http://hz.chenjidiqi.icu/gtxmdhknqc.html

[S04] C：字符串复制
来源：http://hz.yonumen.top/gtzhgtifvp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cheryme.top/gtbavsuknq.html

[S05] C：字符串长度
来源：http://hz.zhoulong.xyz/gtigigtlpd.html

strlen(s)
来源：http://hz.pycfn.com/gtzcrwhecx.html

[S06] C：字符串比较
来源：http://hz.xziqi.cn/gtgjiukkvc.html

strcmp(a, b) == 0
来源：http://hz.dashuyun.cn/gtdgmouiik.html

[S07] C：数组遍历求和
来源：http://hz.yonumen.top/gtlnyomibn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nwbrower.top/gtttteafpm.html

[S08] C：动态内存分配与释放
来源：http://hz.sufxvd.cn/gtmcvwvefs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.daria6918.cn/gtnvjwgmmf.html

[S09] C：结构体定义与初始化
来源：http://hz.iojbl.cn/gtkghpwqsj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cdnleiting.top/gtwfftgusr.html

[S10] C：指针与解引用
来源：http://hz.wangdashe.top/gtgdfvforl.html

int *p = &a;  *p = 5;
来源：http://hz.jyoumei.cn/gtoubjvwhx.html

[S11] C：逐行读文件
来源：http://hz.xziqi.cn/gthmdygxvc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhijiandao.cn/gtxxkbfdmb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj202588.top/gtcavitgfa.html

fclose(f);
来源：http://hz.aizwys.cn/gtwhmlizqe.html

[S12] C：写文件
来源：http://hz.aibaodan.cn/gtwhrsqdyd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hywenlv.cn/gtckwaomwh.html

[S13] C：宏定义
来源：http://hz.xingfuxueyuan.xyz/gtspyyyahh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.bjfxy.top/gthelkggwh.html

[S14] C：枚举
来源：http://hz.xylfe.cn/gtnusraxra.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgfzy.top/gtevnqfdau.html

[S15] C：类型转换
来源：http://hz.ehwqpu.com/gthodindzs.html

(double) a / b
来源：http://hz.chenjidiqi.icu/gtnfavfeeb.html

[S16] C：位操作置位
来源：http://hz.xuetiantiany.cn/gtwztnevrn.html

x |= (1 << 3);
来源：http://hz.wangshuangyany.cn/gtntqkbdgp.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtrrczxjuv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.tian-w.cn/gtboovburg.html

[S18] C：命令行参数
来源：http://hz.svipenyu.cn/gtbjhcsiry.html

int main(int argc, char **argv)
来源：http://hz.xuanzx.com/gtegsllxgs.html

[S19] C：快速排序
来源：http://hz.pengpengdd.cyou/gtefmcdkzw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtvhrqbynl.html

[S20] C：二分查找
来源：http://hz.tian-w.cn/gtlojczcog.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tian-w.cn/gtavqmihrd.html

[S21] C：字符类别判断
来源：http://hz.zhiwuduotai.top/gthtdxtebq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cucudq.cn/gtturoqjrc.html

[S22] C：字符串转数字
来源：http://hz.jiagoushi.top/gtzmczidlh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gzhubu.top/gtmlpwlbuj.html

[S23] C：随机数
来源：http://hz.cdnleiting.top/gtzubciznl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.9152youxi.cn/gtkmykfevg.html

[S24] C：获取本地时间
来源：http://hz.mhx1999.top/gtceanzxyq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zdqjudy.top/gtomhkqphx.html

[S25] C：内存拷贝
来源：http://hz.yueranfly.top/gtrllgrfjs.html

memcpy(dst, src, n);
来源：http://hz.vqdsnc.cn/gtivkirlrw.html

[S26] C：内存清零
来源：http://hz.quarkkingdee.top/gtlifrceji.html

memset(a, 0, sizeof a);
来源：http://hz.shanyushiyangkeji.top/gtdikmbjts.html

[S27] C：定义常量
来源：http://hz.cheryme.top/gtxcyehmis.html

const double PI = 3.14159;
来源：http://hz.ehwqpu.com/gthnzmxkxp.html

[S28] C：静态变量
来源：http://hz.hywenlv.cn/gtvixwldkm.html

static int counter = 0;
来源：http://hz.birdmap.top/gtqrfdnwql.html

[S29] C：变参函数
来源：http://hz.shanyushiyangkeji.top/gtiavvvnuo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hnxiangtu.top/gtvwxidfjj.html

[S30] C：头文件保护
来源：http://hz.shuidangran.top/gtqbhtmbcs.html

#ifndef X_H
来源：http://hz.ppjwa.cn/gtuxhtgnpn.html

#define X_H
来源：http://hz.cucudq.cn/gtzayzpann.html

#endif
来源：http://hz.hnxiangtu.top/gttbrokgjm.html

[S31] C++：Hello World
来源：http://hz.jinqigufen.top/gtbpzngrbt.html

#include <iostream>
来源：http://hz.meibo888.top/gtjiclcjcu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cashguo.top/gtoytvaouh.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtisgglnoi.html

std::string s = "hi";  s += "!";
来源：http://hz.shzxlz.cn/gtyaijxsns.html

[S33] C++：vector 增删
来源：http://hz.tianlin.xyz/gtgtolzsps.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.redwolf501.top/gtpqfpwcvi.html

[S34] C++：遍历 vector
来源：http://hz.chenjidiqi.icu/gtmjbsxaku.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhijiandao.cn/gtrolbmifq.html

[S35] C++：map
来源：http://hz.jinqigufen.top/gtulngzlno.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jqgfzy.top/gtgogzywoa.html

[S36] C++：unordered_map
来源：http://hz.shzxlz.cn/gtiojzneqk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cheryme.top/gtblwctjdv.html

[S37] C++：set
来源：http://hz.wangshuangyany.cn/gtwqrcbkdh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.aibaodan.cn/gtmybkjndl.html

[S38] C++：排序
来源：http://hz.shuidangran.top/gtvmmqubkw.html

std::sort(v.begin(), v.end());
来源：http://hz.pengpengdd.cyou/gtghqsighf.html

[S39] C++：自定义比较器排序
来源：http://hz.redwolf501.top/gtuwkkmonl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cqqwz.cn/gttsgronzo.html

[S40] C++：查找元素
来源：http://hz.cucudq.cn/gttjugczbe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guowangkeji.top/gtizwlryxu.html

[S41] C++：类与构造函数
来源：http://hz.cdnleiting.top/gtnysgqhcc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtnzqndiwy.html

[S42] C++：继承与虚函数
来源：http://hz.gzhubu.top/gtwnesaptz.html

class B : public Base { public: void f() override {} };
来源：http://hz.meibo888.top/gtstdvaqav.html

[S43] C++：智能指针
来源：http://hz.hammf.cn/gtmfhprhfx.html

auto p = std::make_unique<int>(5);
来源：http://hz.cashguo.top/gtlhhtjlzn.html

[S44] C++：引用传参
来源：http://hz.gotoacloud.top/gtpbvxvoac.html

void inc(int &x) { ++x; }
来源：http://hz.sufxvd.cn/gtjdpuckfx.html

[S45] C++：lambda
来源：http://hz.aizwys.cn/gtyedmlrai.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yvedp.cn/gtaxovdfql.html

[S46] C++：函数模板
来源：http://hz.yanxiufei.cn/gtbpujzakg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pengpengdd.cyou/gtqvluamrg.html

[S47] C++：结构化绑定遍历
来源：http://hz.nanxuanxn.top/gtvctwudgn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinyuanbaomall.cn/gtuobnadea.html

[S48] C++：逐行读文件
来源：http://hz.hfpthk.cn/gtotpbhdzf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.kuanghao11.cn/gtpminmder.html

while (std::getline(in, line)) { }
来源：http://hz.gaohongyu789.top/gtgnccfwbf.html

[S49] C++：写文件
来源：http://hz.ehwqpu.com/gtuesexwfl.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aibaodan.cn/gtubgkmovx.html

[S50] C++：格式化数字
来源：http://hz.pycfn.com/gtnlmlgmnk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jianghu66.top/gtewenzwdj.html

[S51] C++：显式类型转换
来源：http://hz.ehwqpu.com/gtaykusotp.html

static_cast<double>(a) / b
来源：http://hz.yj202588.top/gtkrxhvgtr.html

[S52] C++：const 与 noexcept
来源：http://hz.yueranfly.top/gtnwmwfqiv.html

int size() const noexcept { return n_; }
来源：http://hz.jlsjyb.cn/gtkrlggcwe.html

[S53] C++：移动语义
来源：http://hz.ppjwa.cn/gtxhtlyucx.html

std::vector<int> w = std::move(v);
来源：http://hz.chenjidiqi.icu/gtdvtgcais.html

[S54] C++：异常处理
来源：http://hz.haohaochexian.top/gtnmevbgpw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.svipenyu.cn/gtsrxnuxeh.html

[S55] C++：结构化绑定
来源：http://hz.gaohongyu789.top/gtxirocvqy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgufenzy.top/gtaeibzrqq.html

[S56] C++：optional
来源：http://hz.nanxuanxn.top/gtfmawuzya.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cqqwz.cn/gtsjbvoyjp.html

[S57] C++：编译期常量
来源：http://hz.tian-w.cn/gtmzeqrplw.html

constexpr int N = 10;
来源：http://hz.yuanzhike.top/gtfbbsxhof.html

[S58] C++：命名空间
来源：http://hz.hnxiangtu.top/gtwvbvhuox.html

namespace ns { int f() { return 1; } }
来源：http://hz.sufxvd.cn/gtrccjvhlo.html

[S59] C++：静态断言
来源：http://hz.jinqigfzy.top/gtdnbxnguo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jyoumei.cn/gtlocmmwdv.html

[S60] C++：遍历并删除元素
来源：http://hz.cheryme.top/gtkaoxvnoj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhixingplan.top/gtaxhxyney.html

================================================================================
来源：http://hz.ybcxt.top/gtcwpinbnr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.316326.xyz/gtkdhueoso.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtuoklmfsf.html

[T01] Kotlin：Hello World
来源：http://hz.fzhhl.top/gtrmbwpnrf.html

println("Hello")
来源：http://hz.ivvv.top/gtpvlxrfqe.html

[T02] Kotlin：变量
来源：http://hz.shanyushiyangtech.top/gtzhehaktq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.haohaochexian.top/gtcokepoey.html

[T03] Kotlin：字符串模板
来源：http://hz.hysaishi.cn/gttnpxjxkm.html

"值: $b"
来源：http://hz.0kj1m.cn/gtcsvrflvq.html

[T04] Kotlin：空安全
来源：http://hz.nwbrower.top/gteyvwraij.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gtathqxnds.html

[T05] Kotlin：when 表达式
来源：http://hz.bjfxy.top/gtoglyjwwd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shanyushiyangkeji.top/gtgtcegatc.html

[T06] Kotlin：集合映射
来源：http://hz.sysykeji.top/gthnjdgzxs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pengpengdd.cyou/gtghorpxfm.html

[T07] Kotlin：集合过滤
来源：http://hz.yvedp.cn/gtctmvhcky.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cucudq.cn/gtitwamfno.html

[T08] Kotlin：数据类
来源：http://hz.yvedp.cn/gtfgvxsosk.html

data class User(val name: String, val age: Int)
来源：http://hz.yvedp.cn/gtonnlppqn.html

[T09] Kotlin：扩展函数
来源：http://hz.hongshengwenyu.top/gtdstwvxqm.html

fun String.exclaim() = this + "!"
来源：http://hz.dianchejie.cn/gtogzikwxs.html

[T10] Kotlin：默认参数
来源：http://hz.havefunace.top/gtrhrkruwx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.redwolf501.top/gtzbqpxeui.html

[T11] Kotlin：协程
来源：http://hz.sxryk.cn/gtizmjydtr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xingfuxueyuan.xyz/gtftphpznv.html

[T12] Kotlin：解构声明
来源：http://hz.yvedp.cn/gttncquosv.html

val (a, b) = Pair(1, 2)
来源：http://hz.yanxiufei.cn/gtgzmncdpo.html

[T13] Kotlin：只读 Map
来源：http://hz.chenzaomai.com/gtskffbozn.html

val m = mapOf("a" to 1)
来源：http://hz.cashguo.top/gtuetcajcc.html

[T14] Kotlin：循环
来源：http://hz.zhaomingkeji.xyz/gtglupnsxr.html

for (i in 1..10) println(i)
来源：http://hz.gzhubu.top/gtilqjdxkk.html

[T15] Kotlin：接口
来源：http://hz.pycfn.com/gtpbhbzvyo.html

interface Shape { fun area(): Double }
来源：http://hz.zhengqikj.top/gtzrhcfder.html

[T16] Swift：Hello World
来源：http://hz.tianlin.xyz/gtethtlsuq.html

print("Hello")
来源：http://hz.jianghu66.top/gtktjwrphk.html

[T17] Swift：变量与常量
来源：http://hz.jinqigfzy.top/gtpcisyjyz.html

var a = 1;  let b = 2
来源：http://hz.yangfankeji.com/gtnliwnnrl.html

[T18] Swift：字符串插值
来源：http://hz.cashguo.top/gttvlghdox.html

"值: \(b)"
来源：http://hz.iojbl.cn/gtuoautlns.html

[T19] Swift：可选绑定
来源：http://hz.52xcode.cn/gtpjevjphh.html

if let n = opt { print(n) }
来源：http://hz.pengpengdd.cyou/gtimlmgybc.html

[T20] Swift：数组操作
来源：http://hz.fengsongda.top/gtvjvwdkqg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ywan-chungtsiang.top/gttevpjqeb.html

[T21] Swift：遍历
来源：http://hz.zdqjudy.top/gtmlgjkijc.html

for x in a { print(x) }
来源：http://hz.nanxuanxn.top/gtikfwitwl.html

[T22] Swift：字典
来源：http://hz.cqqwz.cn/gttzqwfgea.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hywenlv.cn/gtmgeafiho.html

[T23] Swift：函数
来源：http://hz.xziqi.cn/gtplyfbkgp.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shuidangran.top/gtohdgzwbf.html

[T24] Swift：闭包
来源：http://hz.aibaodan.cn/gtlacbtxli.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xuetiantiany.cn/gtgzygxrxr.html

[T25] Swift：结构体
来源：http://hz.jlsjyb.cn/gtxlcjjbqz.html

struct P { var x: Int }
来源：http://hz.jinqigfzy.top/gtmsqyesvn.html

[T26] Swift：类与重写
来源：http://hz.andypj.xyz/gtkztrwfzt.html

class A: Base { override func f() {} }
来源：http://hz.yj20258.top/gtjrtpmmeg.html

[T27] Swift：错误处理
来源：http://hz.cqqwz.cn/gtieesyzac.html

do { try f() } catch { print(error) }
来源：http://hz.nanxuanxn.top/gtsaazugbn.html

[T28] Swift：枚举
来源：http://hz.mhx1999.top/gtjvtsjlzy.html

enum Color { case red, green }
来源：http://hz.ydjk.org.cn/gtbfnozleq.html

[T29] Swift：guard 提前返回
来源：http://hz.hongshengwenyu.top/gtbtycanhj.html

guard let x = opt else { return }
来源：http://hz.haohaochexian.top/gtowoayhow.html

[T30] Swift：协议
来源：http://hz.gaohongyu789.top/gtbprsxuiw.html

protocol Shape { func area() -> Double }
来源：http://hz.wangdashe.top/gtcmkianee.html

[T31] Lua：Hello World
来源：http://hz.tanke756.top/gtheuqvlrk.html

print("Hello")
来源：http://hz.jyoumei.cn/gtizaytlek.html

[T32] Lua：局部变量
来源：http://hz.zhiwuduotai.top/gtmxbpfyrb.html

local a = 1
来源：http://hz.havefunace.top/gtcbinjyyu.html

[T33] Lua：表（数组）
来源：http://hz.ppjwa.cn/gtubzgiqcv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.dianchejie.cn/gtntmbdmuy.html

[T34] Lua：遍历表
来源：http://hz.guannengcc.top/gtsznwaopl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ivvv.top/gtwodrjpyg.html

[T35] Lua：字典表
来源：http://hz.yj202588.top/gthgkczqlp.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangdashe.top/gtzyecvosb.html

[T36] Lua：函数
来源：http://hz.yangfankeji.com/gtgfwvlzbi.html

function add(a, b) return a + b end
来源：http://hz.mhx1999.top/gtgrijiztp.html

[T37] Lua：字符串拼接
来源：http://hz.tanke756.top/gtkygnsyua.html

"a" .. "b"
来源：http://hz.ywan-chungtsiang.top/gtljzurbrh.html

[T38] Lua：条件
来源：http://hz.jiagoushi.top/gtswxnkkje.html

if x > 0 then print("正") end
来源：http://hz.nwbrower.top/gtumxefxtf.html

[T39] Lua：模式匹配
来源：http://hz.yj20258.top/gtyznbsfdl.html

string.find(s, "%d+")
来源：http://hz.gotoacloud.top/gtyowsvfug.html

[T40] Lua：元表
来源：http://hz.ivvv.top/gtrjawmiiw.html

setmetatable({}, { __index = base })
来源：http://hz.ivvv.top/gtggkwygkn.html

[T41] Perl：Hello World
来源：http://hz.c1oappe.top/gtzwebhyzh.html

print "Hello\n";
来源：http://hz.guowangkeji.top/gtiuwaumco.html

[T42] Perl：变量类型
来源：http://hz.xylfe.cn/gtaffkdnnm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.quarkkingdee.top/gtxhefwosk.html

[T43] Perl：字符串插值
来源：http://hz.zhixingplan.top/gtcdsseimo.html

"值: $a"
来源：http://hz.shangyingyoupin.top/gttquvbjzi.html

[T44] Perl：条件
来源：http://hz.feifeiyinyue.top/gtilwkptxr.html

if ($a > 0) { print "正"; }
来源：http://hz.yonumen.top/gthstwwawx.html

[T45] Perl：数组遍历
来源：http://hz.gogol.net.cn/gtyielnimq.html

for my $x (@arr) { print $x; }
来源：http://hz.vqdsnc.cn/gtwznxlmyk.html

[T46] Perl：哈希操作
来源：http://hz.aibaodan.cn/gtvaesgywq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.316326.xyz/gtiyurdudo.html

[T47] Perl：正则捕获
来源：http://hz.wangdashe.top/gtceqbrkru.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shanyushiyangtech.top/gtquapcguz.html

[T48] Perl：正则替换
来源：http://hz.ehwqpu.com/gttwnezfpn.html

$s =~ s/old/new/g;
来源：http://hz.yj20258.top/gtwfozawmk.html

[T49] Perl：函数
来源：http://hz.nanxuanxn.top/gtyrsosazb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.jianghu66.top/gtmscwbxhg.html

[T50] Perl：逐行读文件
来源：http://hz.iojbl.cn/gtxtszdsty.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.jyoumei.cn/gtdyuwdrxi.html


<!-- 参考信息 -->