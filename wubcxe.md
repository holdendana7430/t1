代发 wailian999

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhmebucs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zcynjptu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2axxpnppc.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2lnbyhywl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2zxfaqzrj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2tvvjtjqb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2axpbvffw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jxlrliwx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qamwrobz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2fotnzbgd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kobgebip.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xposcokb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2sicdrznn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hwcxkajd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xcmnwgtf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2lvbegnbl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2reohemsp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2jheovvfk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hjpbyhok.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ihawolqk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uouolzwm.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xilcjkjv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fvroqime.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pomtatdl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2jrcqdoju.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ikcuiawc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2axsaqudp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tdfxhjuw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2wxnwtlyl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2lsrxnikn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mqidzyiu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2jyyzoyrq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fobrolzk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2guzwppuv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2axgycdvz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kukkpiiz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ubswvfbt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2oodmtghe.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2voqddgkb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hjopsbyi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2isfwfdsh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jkwvczub.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xmvkpmxy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2whlwjbfj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2wmlsjrqx.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rujhvpwh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2yvekifjr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zmqudlpd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vurlrtug.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2teibsuag.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2wglmxvoa.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2weqiepmd.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2mbcamnma.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bhumkvyw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kcfvrxbe.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2cflphvtb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2mqgzpqut.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nvrxgptr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2dpxkmlvd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xohmcbfh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2bolmehsx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wmkkbnhv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vyqbfvum.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2qevwpvjm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2lswnkcsb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2pcmhjsrb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2elflxzdp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2efrzboth.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2blkirmui.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zylcehuj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zumtsnui.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wfxpmzvu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zgechnyl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2lpkcoypi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uusoaerh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2yovtvqed.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2iyobndtt.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2tyszyjfc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2vpgmlpjp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2fseenlzl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fmcfkuke.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2omgevrzj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2etefyzkl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2aqreifqc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2arqmqshp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2oybfzzuv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bkncslck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlkdieua.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tuaenfmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abvjvogm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kuszhnss.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lknoeawo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqsibwal.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2uskqlabx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nlqlzitv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2pobnwleu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ojhlyjgs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2sgcbacbj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wdqklljv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ajnswlwr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kndahzxj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ozxjquzs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xeykevrz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2aclwqagv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cjnhoran.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zmgafxsw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wugfonae.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2brsxnlpt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2qkzqggra.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2aqjxvzpn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2baxgkntv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2haxlzwfi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2czotrndo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kcykmpvl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ddtncwzn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lxocxmbq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2junmhtvj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ikeviyel.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2syocrnkr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pmytqxyb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ysjyzlpi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qmdljwyo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2igvlhffx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rgiobera.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2whksdwce.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kkrocosu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2fjduyqxy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2acfmbzge.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2bfllvjyw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2qvcfhndg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2atanevno.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xqbykjuc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pjjanqnu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lixyafwt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2qrmgrvbh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2gqvkbwxl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dlozjldk.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jyqdzkef.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tdvmxmzx.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rasmhnsr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qebaxcle.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2aisldudm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2hrcmcxqk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nzzcjqno.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zvsjkwne.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2fodbzipe.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yphnhepx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2mxqistux.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2gkdsfome.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2xuixirww.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2yqytmzwv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2phjmbmce.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qvmllxve.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mnsfbiif.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wlepurux.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jxwkzmtf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2mqrmwziy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfmycebu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sqjydxjr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yetyuzlh.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2rxkmvfnv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2tdmafnom.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vzyelmkj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2dzfsgmaz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ugvchvjw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rvripcsp.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2jztgsigu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gpgwkvzr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2roxaxiql.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvfjylpc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2bzogbfew.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nyehgfgu.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2slkybtlm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2keympngx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2gchhdzrc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yvsmbhof.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2mdonqpwy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2rltmvljs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2nibwbgfd.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dwiqrjlr.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ataapabo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jhpsmvoc.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ryimhfvw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qesdmbfv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2opgfoygo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2onlurlvj.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lmncagjc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2golsjlip.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2odmvpnwk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bloicxzk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhddxsyp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2owbrfqqv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nxgzjpig.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzutxvrd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2kttqrebi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2vzslcgmq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nurrphfc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2rtkdkgmf.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2aqagjtgv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2tkffyfop.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2epsnvyov.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2oyximkkp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vrlsltst.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kmcftwio.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2whngvhcl.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2gsgqszuw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mwuwzjtq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2krdgdwhk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwpubkyz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2pbyjpqak.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2tpndrkuq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2twnszoxj.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2nsstraor.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2xqcdrjig.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2mdeayvah.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kkhxjqyj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nkgzbgmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xewymfap.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xgfjfztn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrqfjmws.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xbnmjgjy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mmlietik.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2ymmzaixp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2rumvhuuo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2fxazajho.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2odercewx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2rnhdqqlb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2haeftibv.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2tigeksio.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2envsohuq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2powvudjt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wakvefiw.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2obculajy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xmpamwss.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2zohvxrli.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2qsweyzpj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2trgzelfz.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2wuoleiak.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fcxgtswf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ztmiumrn.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2xryvyryk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2jdhhiohs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2knjiwobp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bzfrkwww.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ropdnzzt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2wqqdyidb.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2wxwphagv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2lcsjgwzj.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2ovnohraa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2xcutcbuo.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wpgvtsso.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kljousde.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xssgdzdk.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2neumpgaq.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2jcxinobq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2thqttarc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ketwssoa.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2vyewygkb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2pinbzhtz.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ddreafxu.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2xmqbycaz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jmjgcnnh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2uurphpga.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2llzbfqeo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2okjwtkhy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2olmeqvht.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mbdtqfsg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2shttfucn.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hdwxsvja.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2jttmnaas.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2cteklanl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2kosvvhpo.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2pvmloxmy.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2osgohtss.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2ergobdmh.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2cydfcdvk.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tybsyrhg.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tfgjyyed.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ixeihrch.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2jlvomgdv.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xkvbpnyt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2zcsdxyes.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2folqjwpv.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2opzrfwbe.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2utbdyleh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2iujadvks.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2pjozcnbr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rkkcnpqo.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ebrsnjxo.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2eidkrsxo.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2bncgkbdf.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2fvdmfpkw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hwcgcbnm.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2tscgecla.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2duwtqlsb.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2hbhtyhht.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2caplpmfl.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rabaddhz.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2pjhvlexc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2gujssgta.html


<!-- 参考信息 -->