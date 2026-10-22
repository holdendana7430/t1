代发 wailian999

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lrqbkkaq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2prjgwdme.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rxjacbly.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2swwilfsq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rgajecez.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mitxeikk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vcgeeasf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nnqszkjq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2sxyjeyvf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lsrkxxiq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2defnnwbj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2novcikrc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2fgkaxovz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2luifievi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2rkciiltq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yovkdgka.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ijjbekxl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vmzjrugl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2irfqkbcu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fypgajvh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2riyjmyfz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ktfmzbuu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gxjxgdfw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ioaogltz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fbmkgjty.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nlmevhld.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sfrhkufe.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2paqdzmrc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hotcclxw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wvpjhkiq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2revoyrww.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ykmrmhhy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2kcahcghz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2adxongnf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zdnfkalk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rgayqivg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2xdyfoyvh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qrkpvfhm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cbsnpicm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ppwjvyoh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vxjxdhlf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rfaqnckt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pmkimhky.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sbceyzkm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hdedvxxr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpksvwzm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2giomzxqz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2hkuoezuj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fntxixny.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2rjueeido.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2smaxmoeb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2oaovevbz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zbpzxfkd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zzpvgudf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fqovgaxy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2diuhrysn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wqskjiis.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2dyqaastp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bahgnkeh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zhocqprz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2typdwzbu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ktvnwzki.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2cgpnwgsl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cdcbyirl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2maqdocdv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2potamcif.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tzjlnyeo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2yxmzmlqj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jwmgrhgv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ipermeqm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uvjgbtxg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mqqlayyj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ksickstw.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2sztailnt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2sqaekogh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lhccbxef.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2isbkrzdf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2mkymegyd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xftgfxuv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jzrmyrek.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2msfonuvm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cguuptta.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cmlvkkvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chxotsck.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qqkqluvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqegrivh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pzirfxwa.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2sqnmxyiv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqmtvjhw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cgfqwrxb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2egqgudmh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2twkkczzo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2qtlbwvux.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2bsddkygc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xqozpjfc.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xoouvaod.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pfhemwjv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2nxrgskji.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fawtshkp.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2rwmdypjc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2biqoluog.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2owtuneut.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2nkbijfdq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dkernuap.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2mckrncsr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mpiyonsn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ohkszvab.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hrtrofgk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2prgrzmjw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xbxarvsk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2evgfweza.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2grxagfzm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bmxxjogn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2cfnadhqx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2cgmrwpja.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2mpyhivum.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2cocugqyg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2plebcjfl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wmcngjbw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nffjjihr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2wnmuhclt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lweproch.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ftqvxncq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fjnrgvrb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2puxuxdmg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2moayjsig.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fpccocnc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2calwbwky.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gqxymmmh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sgnfxhyr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2roegupyx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rqktcchf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2zubjzagk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qizqtcdq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2svtrlxxu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dmqvbfam.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rbldkbjr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2nmwjtobn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2aqvygess.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2tnqvwamf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2sqhbjybv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2tfwlavav.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yhemgenx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2gczhcodh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2acczayis.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2uadrlffj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2zuapjpzk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2tjyfghog.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2todxjbkk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2ycfvzafj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2czvyguws.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hgxzkmct.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mkqyucaw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zfsuzvjw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lfldueqs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2xchvxfuu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rtiznpbr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oqwqwbyb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2qqolloub.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2pzmdmygs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2klwaiged.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hlbmqrgc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2irhvcmcs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qdplqykm.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ffrxjmfd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fmhteayv.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2eswjysnx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fvltwfrt.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2uumpvwpv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2fuprkcau.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ljtdqdcp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xsxdsauh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2qvlvzzxa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lpkyxecc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2qtmkeqjz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2anjtzqcv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2mzfbrwps.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2kcwgghgh.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2ilwjrvrx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxlvltpt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cadtykmf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2yolppbhu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2swkfapit.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpmruagz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2abbughga.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlxnwpoz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2riqhbgwj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ykxllhdb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2zssknnnd.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2mqnjpcli.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ahjicsma.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dqyhmwop.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fxkfswqn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2awjydicr.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2umcysvhh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xdpmxfwx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2wpgedhsg.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sipkwugp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2rltbjjsz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ecridavi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kvtgdzxi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2oyyhnqwk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2ainookxi.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ojfdqzor.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwaysikk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zaztdkxg.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jkzdnesh.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xvypdsza.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fiojdvte.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2mkponlol.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2xawutwfk.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kbgcdbys.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ckjpflsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhzsvcvk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nktnvngp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqbfadeo.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wvnfeipx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2qodgfwde.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2dantywxw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2oxeiwpfg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2iayfoxav.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mwsydeuh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2zivlyelo.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2ypabnqym.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2fvvwqgwb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2mkuhdjdn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2hqrchmab.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2tfyrnmoi.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dfhrhecp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ghzmjgvd.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2czctphqd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2nrousxcu.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2tjbjxyva.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2byyuwctg.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2mamxefyg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kizsjzxx.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2ybtfpvry.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rbfscbkj.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2tgzgxilz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jlqxtueg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2prqvxxah.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2fuxromge.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wkctsicz.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2akhxwruo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2myiwgtdw.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2kgzsilcb.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ceipldmy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2odqnkbej.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2rdixtqow.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uigbhsfb.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vpkwnnai.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2mgtuzqaq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2lcayfchv.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2owpbirxs.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mvgeercm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2kvihfdum.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2eduaqfuf.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2pqtohaqi.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2gjjbhlgi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2cgbqcmyj.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cejytfqc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2dneyibio.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2enemgsrn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2brosddhs.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2rxzjfgmv.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2qkeykysj.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2rofmrtws.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2oamteplm.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2duadigul.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2szicsgul.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2laqtihus.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2emhaimca.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2prtemtty.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ekdeloae.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mtlgnbpw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jljwncpo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cyyzvtmd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ucrdvzbg.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2lomjqosm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wgpqmogm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zzchwgkv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2hpmlqxav.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qgfumrmp.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dbobznbt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2ogwbxupv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eusziwod.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2oushqxcn.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2ygmctppn.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2luiehnhm.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2wvelgbar.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2yzkvtdcs.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2fkozbqle.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2nnzmzcyz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mmvleypw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ucjysvup.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2gdkncpwh.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2iotdkpbj.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2yavuunhi.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2qvaxyayc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yualhkbw.html


<!-- 参考信息 -->