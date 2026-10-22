代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xdsuvauo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vecmtlow.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2oncyehlg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ofbvbhwx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ehotjxxm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2omvpitow.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tnguqomw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2jvkbeyqm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2phftvxya.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2rqhgzifd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2sszwnhbd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nxabufzd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wrddeqpv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ccohpcgd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xwikztnh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kmhzorov.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2afsgoyje.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2nxmfjaac.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zhfmheqw.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2efwswrbd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2diqzzdni.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ozuymgbj.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2txtyyqcf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ikawlcjy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xznbzhyn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2prrfozwn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mxkxufir.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mctyylut.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jcudkkmr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ywitdkdd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ztgokerq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2nnjdahxk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2rwdxwgni.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2nzyilkoy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gtlrcpxq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2qngpydzs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2lvfvkgxw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2rtwypguu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ueuqluzq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wulyiyhm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2xpzgtjqa.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dfsmyxyq.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mzvrsduj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2klththbw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2eubuibaz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wpnosira.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2usrfhwfu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rafwpdjj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2cbeegyvf.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gadoabxb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2jfcgkebj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2esdsslub.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zltzkgsm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2chakpbyg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2scemixly.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mvycczoc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mcqrddup.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ymsohxtk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vmdoilxl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2xetvbfbf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hlmfcckn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wqqnbhtp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wtqhvrwi.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bzgsfchp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gywozlvu.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vusfsmro.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bnojrisk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2arkqtkfc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2lpwisznc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2tnvsbxjb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wjntzvyk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2jdmwogzw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2gmggjrrj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ldzfuwzo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lgxyxszl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wnqcghvn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yptipdmt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kntyldqj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uocmtsja.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ugwcrbxg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2iyojyogx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jlcnbgbf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2yszhfzkt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2spnvismt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2thvxgwzj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2shqacasx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2enoeogtj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2wtcvgkfi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dcsfdknt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2afxyfshr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2qlqsyxku.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qqnirhon.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2yvwkhozo.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2etmgjimd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2lawqlhng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oubckzsv.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nmmsnyzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcqzpiqu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wribeoee.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dcgjdyru.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeqqmcuz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2omgsldja.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2blshtsuk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2tqgydzfc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kliaqqtt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2unihwbap.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2hiwrsnhs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nbngpzig.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xckvrklw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yfrugbar.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pmytmzje.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2edaifpob.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2mxffnqnm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xvcuiyxu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2nxewisng.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jedayblh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dmccglae.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qhtfihgz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dislxlac.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qwutlkkp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2oplnvosi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2hzzlrevb.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rwtuytds.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2jolcfnqi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2msusqsat.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2izgxgciz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2wblcefcl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gpczozff.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ejgrmgdg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bgwavpsn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jbtftnfj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2gtrvcghx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2liyhkxqc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uonzszsb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jcubdrtc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ezxolirn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qhitwfrb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qsynvpjb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sgwpcrle.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2inejurub.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yopjhwor.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ijxppvug.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nyhyrlta.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tpyyaupu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2imakognn.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ixncyeiv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qeuvakxc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2crjmujiz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2lodzkqgz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2itzrddjp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2zzmzjzta.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2vowzilxh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xvkzbndr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2cebalywb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wehffihv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2xgtmqkxl.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wlbxytth.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhkcqmgn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2maexuzyt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2nxbdpkbe.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cqhdiplz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gluzjexr.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2xynnzuwq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zamgxqcu.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jwvghpgb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mtlxaxqs.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2pmqphvgt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2tthegmat.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lcymqris.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2fyvqyqfn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2exscingr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzvfvwsf.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hraibugc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tpurjluv.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2rznjcqhc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lhdvyeyg.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xoafedms.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kwkvqqji.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gcyxtoyb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yoxewice.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cxiyyvam.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2foeotcqf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2wbkobotm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sbepysrz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2edmgyimf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2pgkmwzmu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xjqsoqbt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2kzygokoy.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2dkuijcvp.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2cnravuva.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2xocmkoho.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2ntoazbik.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2scaaqnpx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fbtpwfcd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ajzbcdqj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lztjbjba.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mgfvhrlq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xehoplyb.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dkpowdyd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vqlpfans.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2eohatrls.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wuozozxp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2hfagqwvm.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2btnbcgie.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lxaulolx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qwudotyk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vmrkzxcs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2eaasknuv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2hsaynpji.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2tmurtgtl.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2bshnatgo.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ffwfbbxj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2lnpycvap.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2invoypng.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2vjgvpcsg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2bixoxajh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lbbvhehp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2elvjxeuq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xiessvkq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2nuyizwoo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2xesaoipd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2ijqmxxrf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2oggtoail.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kjbtlypb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2sxkduwgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnjlryof.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2knbocbmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyfhrgbj.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mysyglxq.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lzvuczvz.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2omsaejot.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lujrsupf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2btqukxyw.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2qwlpxbgq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2vjlswvxc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jrlyoipa.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mkriyhur.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jgurzqkz.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ltxnonlz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fjqajejd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gcxalwfh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2joehgrph.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ydbljzqk.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xoazpsxl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2gjbmdpya.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2hizsbyff.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2lhcqpnrc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2bqdvyjyw.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2yranbive.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2owlodove.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rerecocw.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wbxbctpe.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2rmpdgnjq.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsunltkv.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2lgxcenom.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ulzyixyi.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xmoxdqez.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2iglujsqg.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ppwphsfp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2feeelkku.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2zinazbev.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2enqryiib.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mnqwvifa.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ntzfboxm.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2coiacmlr.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2wqfxrjut.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2knwtrwev.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2fxeefdtt.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fdhpldyw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2pmnmtmzf.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hhqukypn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2mojpreig.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ewkoxlxv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2hdwyunqc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2chajuozl.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2czyfpxcz.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2mdzchqpq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2capscblm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2rkluyzti.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hfzdvnzk.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2kucrtsqf.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2yskfihxp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ihimjmeu.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2glaptwmx.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lxjkmgln.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2cjsdkqns.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2mlkxlctx.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2qlkdvppe.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cfyazyxb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2sydekibp.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xktgrzjq.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mpuicktf.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2kbsdgooo.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2jjtkvkcc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2trglqrgg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2dssjsotp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2gbvuyrhj.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2ouejvuqt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qopcdvnb.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bjasnlmi.html


<!-- 参考信息 -->