代发 wailian999

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mgcmqdwf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2pbgxgkwv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2naafdjqt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2wdwwiqcp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vpiwqupe.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ypeoqfmy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sxdzcmde.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2adddajkb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2evqzbuze.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ssioxkju.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kossnddt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pfpluarm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wqeghfod.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qanfuhps.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2shqxknxs.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nhlooqpl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wcaywbju.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2oqeakzfc.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mvgzwcuz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lwjfhkdc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2juwziqnt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2miitcpmr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2exqqoryh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2iadlwmbg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2biinorst.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2fmdgmajb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ethabbvf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bzaghocs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2tslnwgot.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2npkwzsci.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2oseajrag.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pvoerktp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tvowiljm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2iwsyqzew.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2nsksrxfa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2fvjzetud.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vagncybr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pcsbynou.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xzkmijlb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2fzqoegyj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2steeuqpn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2awewpzdy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cmpvlwiy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2clyuuogr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tfgatgvr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vpnbdggo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kwfwcbub.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ypbtluvg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2fkpybbki.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2srlofbyx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pylcuhds.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2rjlueihl.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2rsmswczt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2yzqkdvrr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dhxcsceh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oyfivnul.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2wfoskmqq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dpgswblg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bznessmi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mjcdezmt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2rnffhkxy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2nurmrrcd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2zsogsjvb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2auztldsm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2sqlnfxyf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2imxdvttm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nssbweae.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ygabstdy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pbeklgif.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xrlkxavj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hltwzcus.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xmskxkvg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2civoovli.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2sstsfkpj.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2fkgfbcxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozmrapam.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qnqeirjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brainsob.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kyqxwdch.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2hxaswyeh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2hvwwsgba.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dihzomxm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2twrxwuki.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ftrmmdut.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wzyeiujl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2vfzxuuhz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vaxexetr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gqtdbfwk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nifcynzu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yjnxssbt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2pacwfzex.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2bhkzzrrp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2muflazfw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bljtxucv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2kmruwcjb.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ewzbnfny.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2twfylpdn.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2devjxdml.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ayzvhjze.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bnvldumw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2fwobqzor.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qmwsqpin.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2eqwvsfxm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbjlrnuc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2sikjoarp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2dypohjph.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pfpnbveg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ajvzndmt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2zncrqlyh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qlqbnell.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2quouffgd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qbzuntkn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2revywijy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cobxtvlv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ioskdrog.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cnyidayr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2sqjvamfi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2jexchqsv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fyvvkhab.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bgmkhuhj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2aghacqwp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ojxjptrj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2skiwxqtl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qfbezxsa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2jhcgeyiz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mkhqfbrf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ocorlkch.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2cchwxtjb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2svlmfwer.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jrofdbmx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2fdjwqmfi.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2vbrdkfoh.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2uhfdkpct.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2tbimrxqb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tzizlycz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ltddgofw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2uyxgniiw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2omqbgmgh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wnmnhemc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2vyuojvqo.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ggjcnhqs.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wecyhhgs.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2znehwxxf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gadhunow.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2beqsvsjc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2skfxwfnz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2wdypuopi.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2kmgdcfxm.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ldxgoazd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2hzngwqkt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2avzflndz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xsptvvpj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ljvyaetj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uudcanox.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2dnpqbgmg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wpajwllx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2bjqwiqsn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rqtbcvaj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bxvsqpcr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2epnbaqxl.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zdyzwync.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2mnqwiqfl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2lxbexuuk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2knsnmmfh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gffpaydc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2aaqcmeyy.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2hhzwtbhc.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ysqjhzyt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2koukptsj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sllaefjv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2orkwjxmk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2trdsxjvy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mtvlltwf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fnikzppv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2usmvbmjz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrktymhl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qhblyxby.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2knpytkfd.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktjsmfrw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2xpvchbtj.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bhrtzrvj.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2eyfvlkmy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2derkhmbm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2fqxrsepr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pxdehxvk.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2mpjrjkbu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2mdhxfqum.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2rpgotkjd.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jhiavggz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2cnmeqrkz.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2amqxridc.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2xyqzgumv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ddnpdhkx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2etxkyuxr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vfkhpysd.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2lgnzlfux.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkbiqdxy.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ggacxqtr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mplojxja.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2hheaytyx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qjgdtonb.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2revhqmrz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wqwvygxe.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yevpsbcq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2dmtwmogq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbeapehs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jyupomuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otqukard.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uxzdthsk.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2lftbtkez.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2stqfqvfd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2rinmhiiy.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2wnbxzlac.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2govznyfv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2gkmpcrtk.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2xgoxulrr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2jxhjffmc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2sfnjfupg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2tkwbvglz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2btdeebpz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ejzhtmam.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2oqyrqfio.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jcgmfhut.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2khouyrhx.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2nubhomwo.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2eqnqvrea.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qiqvfbto.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2yvcmcmna.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2aprdffth.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jyfewyxf.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2habxcgwy.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzlkmkrp.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rffhqais.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2dgyopysv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2aydmskho.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2gwmthkzg.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2smdlulsk.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jdvfwyil.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2shdiwkza.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2styrfkrc.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2edrziqfh.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2bpvyymtz.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qbretaka.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2oetmlcns.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fixpuhae.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2ipzcutaf.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2mtnqecpn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2smkmtlse.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fxnxvtoc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zzhbeicp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vfnoyyji.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2dixhthtl.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2iqlebfls.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2undsbviv.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2gpqulcrn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2llivegup.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2nthmcdvy.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2bpvzbgaz.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ezhcmdsa.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tlpbxnnq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pcwycqaj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2pykgnlec.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2esomiuor.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2uwbxemrb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2lsijfmkb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2cvapflhj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2biqaqpnc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2djtlvrel.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hrisaomh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ijordhmp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2uiicxqog.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uexlukrw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2syqucrza.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dicqwqdt.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2efxnnwii.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ozygtwvr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2tlueyccs.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2iuyfhqsi.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wdnrdkzb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lhveeemp.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2msbgszjc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2xssxmyzf.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2tgzhnypd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gsjvxukk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vtzmvlir.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ccpnbjxr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2nwhwtujj.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2kcujjnal.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fjriwnzh.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mmcphhbh.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2linoohel.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2volqglfj.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2oddspioi.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2bdgfvhih.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2laiiwnho.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozuabadv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kzmlxubw.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjujhrbv.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2sjtdqglj.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2uwlxotkx.html


<!-- 参考信息 -->