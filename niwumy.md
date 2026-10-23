代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3juqixiay.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3entntvfq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lrjgmoov.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3oiwnpksg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wankjmhw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rhqhjjuv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cmpwwcml.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xdsudndn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jdbseqys.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3noivlpqd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3alrdvnqx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nzalxpac.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3krkvkttj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3anhrcgjs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3urbxnptk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3jgprxxww.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vktfglse.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3idvfvkgh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3immiaxpm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zowkrggf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3bkrsdrsy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tvavjpcw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3cuzlrrqe.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nclyrcoq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3gqmdwjdv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eqzcsnwp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3baeeedod.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jjprtifq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3sqwzbnde.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxyszxzh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vswbcepn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pqbcoepl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xewqwkkm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vfeqvejz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3zjrkmtfx.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3pvmqcknw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3hazbftga.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3qqqhlcbt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3fpimwuib.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ldutagdm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jryradee.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vdpfspsd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3httfsumb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3lijcrrcm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3euqgnoqm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3wjhefeyy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3jybnxqwq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xingqsur.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rgcvifgc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fgwbnmls.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ezmjzgxp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3niveiuwq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3vzpokfsi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ulrzgdnm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3fcivgamx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hctvfowy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3tdjjspkr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bgokvhun.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fpuwhoag.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ndbilxbu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3tkekwjjx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qxoweuli.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kbfpqmin.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3libobdfl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3tcmhawbu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3myymixjm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3eqrqjnvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzxbcjer.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ffrzsibn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtajppzp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3myvsmvug.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vvkbpqvq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3finzuxsp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kacachrz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3asagxkdp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3klfiujis.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kgmzwivr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3pldpjpov.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lemejctx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jbhbpmnj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpqqipnc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jabkmsbo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cyodgzwn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3luzzcwnl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qumqzirj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tdsfojwc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3yysjgnfr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3nzarhjrn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3nfuwvsbb.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mksbzkez.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3gnvncxsy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3knymkrdz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3esapsqno.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gnkbttom.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uiemytae.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vpebptid.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3thafekgr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rsnbctvv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ummnxtmc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3gjcgpgjl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3upbnbpad.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3jjavjeuh.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3neljkstf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nnmmzbxf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ldkyfqsd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dhffmnjb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mfukyyic.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3skuxtmkw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xfesvygo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3wksgizzy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qfhhfrsw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3htjunapk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3wokrgyvh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3qluxilpo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3yvkhirxr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yfqigqhc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3zqbssktw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3rmntiygs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hgnymelo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mkopqkla.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3kubiltrm.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3auyhlcbr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3nyqmkpgq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3tmvlqged.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rgbabmlo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3syzmynuz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jgcxjxni.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xnvpzaby.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3egkaechm.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3jinfhjtl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3zujdwbjh.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3udztxcwk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3fztkrdwy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dpoyfjtt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3ntsvytwp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvyrftji.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3iemqobjf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gouvghqc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3chturzbb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3omqxbzgz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vxvmtxft.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3stqmczdb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ylvbjwvo.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yspfloeo.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3jxtedqqx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gyhwukuo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3unvfomtl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kakmbbsg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3trspliqu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zmhudhkx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zzgbmvus.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fhgbgtur.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3lgbnupfb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3govokqlq.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3ccixcwdh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3onptaudx.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3dluaadcy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3xvzlbadd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3xtdsvwsl.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ezzssbwc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cjzfexbk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qulsfmyf.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3yczpagxs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3afgvdwwu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tnbxnbeq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3julspmrp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fazrzujb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxuzwlgi.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3uozkpiln.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkijqbqb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jrinshua.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3dqzeamgw.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qvjgyaxi.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3qwavlgfz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3kfftkatz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3rtzjnsib.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rfrbwpop.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tmvbdott.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ytgplrsh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3kvesbkqy.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3fedfjudn.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gxtprfpq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3nwguxcsd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3gvrrkuun.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jpyvawuz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3asbpjlot.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eutcabqt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3uyrapvvw.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3redxjtzd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3yrjsyqxi.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3sdcgvtjs.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ourfbcby.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rsuwmqoh.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3jwdstqhg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3gpfktzly.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3lzcutwdd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xdrobkjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmirjgfs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xldrkrah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbemvlpe.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gubspbtl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3yuhhtaon.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3ykqbwasv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mpdmjpgj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3djyfrfpr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sibochar.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3lwntlaol.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3osftmqaw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3mhjxyubf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3clmdngqu.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ftgjxfos.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pnloixnz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3aqsquxjb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3jwjtdbnx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ycfuecvf.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xwsfsfvl.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbblnpua.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3aweiodeh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3zsiolxhg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3rbmwplry.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3uxieytel.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3zxhupgep.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jclzdsbd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tpfacfip.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3kdlrhlrl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywctbntn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fgquucum.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3knicozyl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3ndhyehdp.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3oixualqu.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ahwqecyg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3fhtsgcpe.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3jbttldtf.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xbspytia.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3obllrkmf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3ttzuxdyc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3zpjnkfbg.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3xcnvftkl.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ajrmylnj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3iijdougs.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ufmaokoi.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3wgseuvxl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3sbwajmuo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3cahkhmew.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ipaqulsf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vtdidwxw.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kxnkaysw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kvdhuknt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3xwnfwphr.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3vxrpwakr.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3pvonlcar.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jfwutgco.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kipwnnyd.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3rdpwcfjg.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3limprdsw.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3glcwfxzc.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3dcqdovpj.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3gocczykk.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3ghjsyfqn.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ryypjjeo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cwivdegi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3bawievsz.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rfgcckhi.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3phrjwxwp.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3vkmzcveo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3bpxmgcmd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3ixmjnyzo.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3pchnybwm.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3byfzczjt.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zdyduols.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3jaunhpxd.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3nquwtvwr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3nxwhugpy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3vdwvqfvk.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3zbofruuo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3jmctkcuw.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3shqznrur.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3aikhbpau.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3drfalwku.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3tpmcnwye.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xjnmwidn.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3asgckrci.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxhljhvt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3wkohdldp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vboztvwp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3rgifuscv.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3fchcjact.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwgbrsgm.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3corzpoep.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3qirqnsbe.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3zallwpuw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltgngouf.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bhqnenlb.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wydzeljn.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3crpaxmzj.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3vwbtpstb.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nftodsxb.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukzljgnb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mnipoqig.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3pdxolihi.html


<!-- 参考信息 -->