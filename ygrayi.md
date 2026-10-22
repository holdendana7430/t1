代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ynptinvd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2dhjsmlri.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jhpxghcf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2gpxypirr.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2iybdihuz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yrcegiel.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ndqadbmd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2spqzyhim.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lxdxpinj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rexwzbjj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2knebliyr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zrjwgljc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vrerxiar.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dfnvhbpw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ntlgnkjh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2fhtcybvq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kitxfkyt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2qoyukcnq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2tscwnbma.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2pdcwnqaw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2crensbjz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2piyjegwd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2uipovnvg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ijwtscks.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qspfnbyo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2chpsuqmj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2frsfemtl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dkpfxzwz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xslttaom.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rynmfdun.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kfsjbjcy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tsfwdhac.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ggxshdaz.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qzrlzirr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dbsmymow.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2yupvuplj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2oadljevn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwqsbvnt.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2yvqwkzoy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qeyjoeew.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2lcaeecog.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gzrzxtzj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ktevvkgw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2swqpvcyl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2lxyqnxua.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2cojoozlt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2abeuliac.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pjgcimsp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ddryfjjn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tzktagtu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gebfmtcm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nlsiiiob.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2pixztwbh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hshzzlcp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2kxzfvjlt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2qnyvybab.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2tptvhvqj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2cqvaspjv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2usrscmgv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lkjfhlap.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fhqcvsgz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ftwhmblr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2cmdflmfh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jjrfcrvz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2uqwrtzoc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2jfvbxuxp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2dkiozhxp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fspzrueg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2dgxwzyja.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2eqfpzkvu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2khzudbez.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mmoytqdr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2buwbcnxj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lydnvnjh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zfitrhqs.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xlnvdmmr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2fnattbkn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xzkkfqff.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2klsuvcop.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2gpclwzht.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2rxwmrwna.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zjljsuiq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ahnychhk.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2smezlfgt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pvafenod.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2onsvahcr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2klldqdzs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bnjmmyen.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2tgsqhgdh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ljkzhlcb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zhayqhtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kyvywnbq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xxspxtwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adouvzjy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lwweiyae.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fmxvyduq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cazzoltq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xxiragqw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ymwhcouk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ompmruti.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cwjzelye.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ttclivlr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2dgjydftg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pohxcdud.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sfujwpkt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bhrkgeog.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2noojewzb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2wxzsctws.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xkxxedoz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2sovufzev.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2kzqmnqjy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ophrzsii.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cgpzcovt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tsyusnwj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ynrkqvrp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfogzswi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2glcnovju.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2oklsaqni.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ixwlczka.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2smjtkhmt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gwcpribv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2lujhjcim.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rzphhrhr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zldtfehe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ycztrhki.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ccyurxeo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xdajbnel.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2pzhqmbqg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qmmoxjzb.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ikibzzcg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2nrdscljr.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jutmehve.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jtlflfzc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2pockkwrc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jquqquzi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2opxniowi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dtfvloub.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2pdbstatx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2cebhibsz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2nagoxnwf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2fzfydcti.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wtdjdxva.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cpzqajwk.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2geemxnvp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2zzmkmvup.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2lqpmyvhp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2dgihltph.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2wifldzhn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ykuqzlfc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2obhcusbl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ttdiquxv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2lraajkww.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2atgbtifb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2rbjkrbpe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fvgucvst.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ixrrotcd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wzxmkrkf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2fmuuukzn.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2dfdymdqj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ejuavwnz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2cwkrvpqz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2cxadekzp.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gdfkyfhp.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2eoybesnb.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2sgimlqgc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2feitngry.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2mruavkvh.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyxtcbbb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2dncugdlj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2slcoxbdl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lqrushwc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bcrzstzt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2smyjvgxh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2urlrtfch.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ouaklxct.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pqbdwrjn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2tubmxlcv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ruqkurpm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yernlhmt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2xoghbtjm.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2mvymjuby.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2zhdaxmbo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2azpptnaj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2oeuibhif.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2brssygbk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2dnbcpyuo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2bbtqfmll.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fcifvygt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2tjnmflwl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fwxnqedt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2upzoefnd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ornknylh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2pjunagtt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeqekywh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lmpnltwa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2djlolnjt.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kiywozdk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrtmhfde.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rbrcvzkg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2lsbbtfac.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2agjwchbq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2mfvaxcbw.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2znjfazln.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2pglkdgru.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ipccrnef.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2hczlgweq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2egharkno.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fywtxbez.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2icmknkzq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2pxyztxyp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2lcedmvgv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2bcohnwdc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozeyatha.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2toiucphf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2opjkbzvn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mwrxqlkp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sxjaoksl.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2erfisgih.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2aiythcjf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2vwqhltva.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2qdjibqcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbovqgvq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2slcvkgzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctlvqvgc.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yhhhljbg.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nxfrpvja.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2folwneyj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bsdkosvl.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2bauzwzqt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2lbxzyovx.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2hkexwobr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2cairdsrv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tpvvmrkx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2itxxunxe.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2etbttiij.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzixrsg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zggjucwx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2tdwvgxtr.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2jgxiaobv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2ztckcwid.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2csnddssy.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2pcgatfow.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2egifhkjc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2bmfzctqb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2atbhlcmr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2rhtcnjpl.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2tepbuund.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fdwpridq.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2rrqwhssf.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2svnaxima.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2aodwdknj.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nrcugduy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2pnhkvacj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2oymasblv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hdrjfune.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tkannjwc.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2nzebtvwe.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2lyqzgovm.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bzfadmob.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2lrnwyofc.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wngyxnns.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2izzgyyeq.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2vpmljvfg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jxjjyclg.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2kukqycot.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2cbwrtrex.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2qgrmotgn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2vzlwdhrh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ygsejtnz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ugqvshhc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2efsqdikx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bhgurkbz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2oijsruhg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2elugippg.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2nmnatxgl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2tdiqusix.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ifncskeb.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2ubcspuom.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2uqnnprmk.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2jeppesic.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ylxblzbn.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uasctjli.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2juyyyrlr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2onrgoamq.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dskrvwgq.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2vsdvtvvk.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2cmkgjmhu.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvznmvip.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dbtkdrst.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2oqhzlsyj.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2luznnujb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ufsfkwry.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ldrkrpud.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2hljlcije.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2pmkgmtds.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2znwdrxdb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ccbcflzb.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2fgbgehrq.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2ofvhdfqo.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2bavtbsfv.html


<!-- 参考信息 -->